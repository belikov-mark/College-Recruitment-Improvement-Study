# College Recruitment Improvement Study
 
The purpose of the study is help improve college recruiments. 

{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "03ea9a33",
   "metadata": {},
   "source": [
    "Mark Belikov"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "6a591a07",
   "metadata": {},
   "source": [
    "2/23/2024"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "f246657d",
   "metadata": {},
   "outputs": [],
   "source": [
    "#importing pandas and plots to show graphs"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 2,
   "id": "a98d777b",
   "metadata": {},
   "outputs": [],
   "source": [
    "import pandas as pd"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 7,
   "id": "5755392a",
   "metadata": {},
   "outputs": [],
   "source": [
    "import matplotlib.pyplot as plt"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "fc8a13cd",
   "metadata": {},
   "outputs": [],
   "source": [
    "#reads file"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 8,
   "id": "7b261e10",
   "metadata": {},
   "outputs": [
    {
     "ename": "ParserError",
     "evalue": "Error tokenizing data. C error: Expected 1 fields in line 4, saw 2\n",
     "output_type": "error",
     "traceback": [
      "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
      "\u001b[1;31mParserError\u001b[0m                               Traceback (most recent call last)",
      "Input \u001b[1;32mIn [8]\u001b[0m, in \u001b[0;36m<cell line: 1>\u001b[1;34m()\u001b[0m\n\u001b[1;32m----> 1\u001b[0m file \u001b[38;5;241m=\u001b[39m \u001b[43mpd\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mread_csv\u001b[49m\u001b[43m(\u001b[49m\u001b[38;5;124;43m'\u001b[39;49m\u001b[38;5;124;43mUntitled1.IPYNB\u001b[39;49m\u001b[38;5;124;43m'\u001b[39;49m\u001b[43m)\u001b[49m\n",
      "File \u001b[1;32m~\\anaconda3\\lib\\site-packages\\pandas\\util\\_decorators.py:311\u001b[0m, in \u001b[0;36mdeprecate_nonkeyword_arguments.<locals>.decorate.<locals>.wrapper\u001b[1;34m(*args, **kwargs)\u001b[0m\n\u001b[0;32m    305\u001b[0m \u001b[38;5;28;01mif\u001b[39;00m \u001b[38;5;28mlen\u001b[39m(args) \u001b[38;5;241m>\u001b[39m num_allow_args:\n\u001b[0;32m    306\u001b[0m     warnings\u001b[38;5;241m.\u001b[39mwarn(\n\u001b[0;32m    307\u001b[0m         msg\u001b[38;5;241m.\u001b[39mformat(arguments\u001b[38;5;241m=\u001b[39marguments),\n\u001b[0;32m    308\u001b[0m         \u001b[38;5;167;01mFutureWarning\u001b[39;00m,\n\u001b[0;32m    309\u001b[0m         stacklevel\u001b[38;5;241m=\u001b[39mstacklevel,\n\u001b[0;32m    310\u001b[0m     )\n\u001b[1;32m--> 311\u001b[0m \u001b[38;5;28;01mreturn\u001b[39;00m func(\u001b[38;5;241m*\u001b[39margs, \u001b[38;5;241m*\u001b[39m\u001b[38;5;241m*\u001b[39mkwargs)\n",
      "File \u001b[1;32m~\\anaconda3\\lib\\site-packages\\pandas\\io\\parsers\\readers.py:680\u001b[0m, in \u001b[0;36mread_csv\u001b[1;34m(filepath_or_buffer, sep, delimiter, header, names, index_col, usecols, squeeze, prefix, mangle_dupe_cols, dtype, engine, converters, true_values, false_values, skipinitialspace, skiprows, skipfooter, nrows, na_values, keep_default_na, na_filter, verbose, skip_blank_lines, parse_dates, infer_datetime_format, keep_date_col, date_parser, dayfirst, cache_dates, iterator, chunksize, compression, thousands, decimal, lineterminator, quotechar, quoting, doublequote, escapechar, comment, encoding, encoding_errors, dialect, error_bad_lines, warn_bad_lines, on_bad_lines, delim_whitespace, low_memory, memory_map, float_precision, storage_options)\u001b[0m\n\u001b[0;32m    665\u001b[0m kwds_defaults \u001b[38;5;241m=\u001b[39m _refine_defaults_read(\n\u001b[0;32m    666\u001b[0m     dialect,\n\u001b[0;32m    667\u001b[0m     delimiter,\n\u001b[1;32m   (...)\u001b[0m\n\u001b[0;32m    676\u001b[0m     defaults\u001b[38;5;241m=\u001b[39m{\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mdelimiter\u001b[39m\u001b[38;5;124m\"\u001b[39m: \u001b[38;5;124m\"\u001b[39m\u001b[38;5;124m,\u001b[39m\u001b[38;5;124m\"\u001b[39m},\n\u001b[0;32m    677\u001b[0m )\n\u001b[0;32m    678\u001b[0m kwds\u001b[38;5;241m.\u001b[39mupdate(kwds_defaults)\n\u001b[1;32m--> 680\u001b[0m \u001b[38;5;28;01mreturn\u001b[39;00m \u001b[43m_read\u001b[49m\u001b[43m(\u001b[49m\u001b[43mfilepath_or_buffer\u001b[49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[43mkwds\u001b[49m\u001b[43m)\u001b[49m\n",
      "File \u001b[1;32m~\\anaconda3\\lib\\site-packages\\pandas\\io\\parsers\\readers.py:581\u001b[0m, in \u001b[0;36m_read\u001b[1;34m(filepath_or_buffer, kwds)\u001b[0m\n\u001b[0;32m    578\u001b[0m     \u001b[38;5;28;01mreturn\u001b[39;00m parser\n\u001b[0;32m    580\u001b[0m \u001b[38;5;28;01mwith\u001b[39;00m parser:\n\u001b[1;32m--> 581\u001b[0m     \u001b[38;5;28;01mreturn\u001b[39;00m \u001b[43mparser\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mread\u001b[49m\u001b[43m(\u001b[49m\u001b[43mnrows\u001b[49m\u001b[43m)\u001b[49m\n",
      "File \u001b[1;32m~\\anaconda3\\lib\\site-packages\\pandas\\io\\parsers\\readers.py:1254\u001b[0m, in \u001b[0;36mTextFileReader.read\u001b[1;34m(self, nrows)\u001b[0m\n\u001b[0;32m   1252\u001b[0m nrows \u001b[38;5;241m=\u001b[39m validate_integer(\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mnrows\u001b[39m\u001b[38;5;124m\"\u001b[39m, nrows)\n\u001b[0;32m   1253\u001b[0m \u001b[38;5;28;01mtry\u001b[39;00m:\n\u001b[1;32m-> 1254\u001b[0m     index, columns, col_dict \u001b[38;5;241m=\u001b[39m \u001b[38;5;28;43mself\u001b[39;49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43m_engine\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mread\u001b[49m\u001b[43m(\u001b[49m\u001b[43mnrows\u001b[49m\u001b[43m)\u001b[49m\n\u001b[0;32m   1255\u001b[0m \u001b[38;5;28;01mexcept\u001b[39;00m \u001b[38;5;167;01mException\u001b[39;00m:\n\u001b[0;32m   1256\u001b[0m     \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mclose()\n",
      "File \u001b[1;32m~\\anaconda3\\lib\\site-packages\\pandas\\io\\parsers\\c_parser_wrapper.py:225\u001b[0m, in \u001b[0;36mCParserWrapper.read\u001b[1;34m(self, nrows)\u001b[0m\n\u001b[0;32m    223\u001b[0m \u001b[38;5;28;01mtry\u001b[39;00m:\n\u001b[0;32m    224\u001b[0m     \u001b[38;5;28;01mif\u001b[39;00m \u001b[38;5;28mself\u001b[39m\u001b[38;5;241m.\u001b[39mlow_memory:\n\u001b[1;32m--> 225\u001b[0m         chunks \u001b[38;5;241m=\u001b[39m \u001b[38;5;28;43mself\u001b[39;49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43m_reader\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mread_low_memory\u001b[49m\u001b[43m(\u001b[49m\u001b[43mnrows\u001b[49m\u001b[43m)\u001b[49m\n\u001b[0;32m    226\u001b[0m         \u001b[38;5;66;03m# destructive to chunks\u001b[39;00m\n\u001b[0;32m    227\u001b[0m         data \u001b[38;5;241m=\u001b[39m _concatenate_chunks(chunks)\n",
      "File \u001b[1;32m~\\anaconda3\\lib\\site-packages\\pandas\\_libs\\parsers.pyx:805\u001b[0m, in \u001b[0;36mpandas._libs.parsers.TextReader.read_low_memory\u001b[1;34m()\u001b[0m\n",
      "File \u001b[1;32m~\\anaconda3\\lib\\site-packages\\pandas\\_libs\\parsers.pyx:861\u001b[0m, in \u001b[0;36mpandas._libs.parsers.TextReader._read_rows\u001b[1;34m()\u001b[0m\n",
      "File \u001b[1;32m~\\anaconda3\\lib\\site-packages\\pandas\\_libs\\parsers.pyx:847\u001b[0m, in \u001b[0;36mpandas._libs.parsers.TextReader._tokenize_rows\u001b[1;34m()\u001b[0m\n",
      "File \u001b[1;32m~\\anaconda3\\lib\\site-packages\\pandas\\_libs\\parsers.pyx:1960\u001b[0m, in \u001b[0;36mpandas._libs.parsers.raise_parser_error\u001b[1;34m()\u001b[0m\n",
      "\u001b[1;31mParserError\u001b[0m: Error tokenizing data. C error: Expected 1 fields in line 4, saw 2\n"
     ]
    }
   ],
   "source": [
    "file = pd.read_csv('Untitled1.IPYNB')"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "fd628801",
   "metadata": {},
   "outputs": [],
   "source": [
    "#Questions"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "069184d7",
   "metadata": {},
   "outputs": [],
   "source": [
    "1. What is the intrests of students for taking computing classes?\n",
    "\n",
    "2. Is there a correleation between a students academic performance and intrest in computing classes?"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "dd02e418",
   "metadata": {},
   "outputs": [],
   "source": [
    "#plots for the questions"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "a6aa0b93",
   "metadata": {},
   "outputs": [],
   "source": [
    "plt.figure(figsize=(10,5))\n",
    "plt.xlabel('Interest in class')\n",
    "plt.ylabel(\"Number of students\")\n",
    "plt.show"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "db32e32a",
   "metadata": {},
   "outputs": [],
   "source": [
    "plt.figure(figsize=(10,5))\n",
    "plt.xlabel('Academic perfomance')\n",
    "plt.ylabel(\"Interest in class\")\n",
    "plt.show"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "63788c52",
   "metadata": {},
   "outputs": [],
   "source": [
    "3. What are the most likely choices of a major after the computing major to enroll in computing course?\n",
    "\n",
    "4. Is there a specific race, gender, age that there are more of that are enrolled in a computing class?"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "57c929b8",
   "metadata": {},
   "outputs": [],
   "source": [
    "plt.figure(figsize=(10,5))\n",
    "plt.xlabel('Majors')\n",
    "plt.ylabel(\"Number of students\")\n",
    "plt.show"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 9,
   "id": "19fdb243",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "<function matplotlib.pyplot.show(close=None, block=None)>"
      ]
     },
     "execution_count": 9,
     "metadata": {},
     "output_type": "execute_result"
    },
    {
     "data": {
      "image/png": "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\n",
      "text/plain": [
       "<Figure size 720x360 with 1 Axes>"
      ]
     },
     "metadata": {
      "needs_background": "light"
     },
     "output_type": "display_data"
    }
   ],
   "source": [
    "plt.figure(figsize=(10,5))\n",
    "plt.xlabel('Race')\n",
    "plt.ylabel(\"Number of students\")\n",
    "plt.show"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 10,
   "id": "e4750182",
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "<function matplotlib.pyplot.show(close=None, block=None)>"
      ]
     },
     "execution_count": 10,
     "metadata": {},
     "output_type": "execute_result"
    },
    {
     "data": {
      "image/png": "iVBORw0KGgoAAAANSUhEUgAAAmkAAAFBCAYAAAAsZjgUAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAAAsTAAALEwEAmpwYAAAYdklEQVR4nO3de7BlZX3m8e9jo1GQixHiaANKHAzBCjh6REuMgLcAGlBLa8DbDFJBasDgOClBy6AjU6UWQaMB7LSGoE7KTiSUgtOIZkpxohLpVu6K6aBCixHwBoESquE3f+zVYXM8l9Wne51+d+/vp2rX2Wutd73nB29119PvurypKiRJktSWR2zvAiRJkvTrDGmSJEkNMqRJkiQ1yJAmSZLUIEOaJElSgwxpkiRJDRospCW5IMntSa6f53iSfCTJhiTXJnnmULVIkiRNmiFn0i4Ejlzg+FHA/t3nJOCjA9YiSZI0UQYLaVX1VeBnCzQ5FvhkjVwJ7JHkiUPVI0mSNEm25z1pK4Fbx7Y3dvskSZKm3k7b8Xdnjn1zrlGV5CRGl0TZZZddnnXAAQcMWZckSdI2sX79+juraq+lnLs9Q9pGYJ+x7b2B2+ZqWFWrgdUAMzMztW7duuGrkyRJ2kpJfrjUc7fn5c5LgDd2T3k+F/hlVf14O9YjSZLUjMFm0pJ8Gjgc2DPJRuDdwCMBqmoVsBY4GtgA3AucMFQtkiRJk2awkFZVxy9yvIBThvr9kiRJk8wVByRJkhpkSJMkSWqQIU2SJKlBhjRJkqQGGdIkSZIaZEiTJElqkCFNkiSpQYY0SZKkBhnSJEmSGmRIkyRJapAhTZIkqUGGNEmSpAYZ0iRJkhpkSJMkSWqQIU2SJKlBhjRJkqQGGdIkSZIaZEiTJElqkCFNkiSpQYY0SZKkBhnSJEmSGmRIkyRJapAhTZIkqUGGNEmSpAYZ0iRJkhpkSJMkSWqQIU2SJKlBhjRJkqQGGdIkSZIaZEiTJElqkCFNkiSpQYY0SZKkBhnSJEmSGmRIkyRJapAhTZIkqUGGNEmSpAYZ0iRJkhpkSJMkSWqQIU2SJKlBhjRJkqQGGdIkSZIaZEiTJElqkCFNkiSpQYY0SZKkBhnSJEmSGmRIkyRJatCgIS3JkUluSrIhyRlzHN89yaVJrklyQ5IThqxHkiRpUgwW0pKsAM4DjgIOBI5PcuCsZqcAN1bVwcDhwDlJHjVUTZIkSZNiyJm0Q4ANVXVzVd0PrAGOndWmgF2TBHgs8DNg04A1SZIkTYQhQ9pK4Nax7Y3dvnHnAr8L3AZcB5xWVQ/O7ijJSUnWJVl3xx13DFWvJElSM4YMaZljX83a/gPgauBJwDOAc5Ps9msnVa2uqpmqmtlrr722dZ2SJEnNGTKkbQT2Gdvem9GM2bgTgItrZAPwfeCAAWuSJEmaCEOGtKuA/ZPs1z0McBxwyaw2twAvAkjyBOB3gJsHrEmSJGki7DRUx1W1KcmpwOXACuCCqrohycnd8VXAWcCFSa5jdHn09Kq6c6iaJEmSJsVgIQ2gqtYCa2ftWzX2/TbgpUPWIEmSNIlccUCSJKlBhjRJkqQGGdIkSZIaZEiTJElqkCFNkiSpQYY0SZKkBhnSJEmSGmRIkyRJapAhTZIkqUGGNEmSpAYZ0iRJkhpkSJMkSWqQIU2SJKlBhjRJkqQGGdIkSZIaZEiTJElqkCFNkiSpQYY0SZKkBhnSJEmSGmRIkyRJapAhTZIkqUGGNEmSpAYZ0iRJkhpkSJMkSWqQIU2SJKlBhjRJkqQGGdIkSZIaZEiTJElq0KIhLclpSXbLyF8l+VaSly5HcZIkSdOqz0zam6rqLuClwF7ACcD7B61KkiRpyvUJael+Hg38dVVdM7ZPkiRJA+gT0tYn+SKjkHZ5kl2BB4ctS5Ikabrt1KPNicAzgJur6t4kj2d0yVOSJEkD6TOT9qWq+lZV/QKgqn4KfGjQqiRJkqbcvDNpSR4N7AzsmeRxPHQf2m7Ak5ahNkmSpKm10OXONwNvZRTI1vNQSLsLOG/YsiRJkqbbvCGtqj4MfDjJW6rqL5axJkmSpKm36IMDVfUXSZ4HPGW8fVV9csC6JEmSptqiIS3Jp4CnAlcDD3S7CzCkSZIkDaTPKzhmgAOrqoYuRpIkSSN9XsFxPfAfhi5EkiRJD+kzk7YncGOSbwL3bd5ZVccMVpUkSdKU6xPS3jN0EZIkSXq4Pk93XpHkycD+VfUPSXYGVgxfmiRJ0vRa9J60JH8EXAT8ZbdrJfDZAWuSJEmaen0eHDgFOJTRSgNU1T8Dv9Wn8yRHJrkpyYYkZ8zT5vAkVye5IckVfQuXJEnakfW5J+2+qro/Ga0KlWQnRu9JW1CSFYyWj3oJsBG4KsklVXXjWJs9gPOBI6vqliS9wp8kSdKOrs9M2hVJ3gk8JslLgM8Al/Y47xBgQ1XdXFX3A2uAY2e1eS1wcVXdAlBVt/cvXZIkacfVJ6SdAdwBXMdo0fW1wLt6nLcSuHVse2O3b9zTgMcl+UqS9Une2KNfSZKkHV6fpzsfBD7WfbZE5upujt//LOBFwGOAbyS5sqq+97COkpOAkwD23XffLSxDkiRp8swb0pJcxwL3nlXVQYv0vRHYZ2x7b+C2OdrcWVX3APck+SpwMPCwkFZVq4HVADMzMy5PJUmSdngLzaS9vPt5SvfzU93P1wH39uj7KmD/JPsBPwKOY3QP2rjPAed2DyM8CngO8KEefUuSJO3Q5g1pVfVDgCSHVtWhY4fOSPI14L0LdVxVm5KcClzO6OW3F1TVDUlO7o6vqqrvJPkCcC3wIPDxqrp+6/6TJEmSJl+fV3DskuT5VfWPAEmeB+zSp/OqWsvoQYPxfatmbZ8NnN2vXEmSpOnQJ6SdCFyQZPdu+xfAmwarSJIkSb2e7lwPHJxkNyBV9cvhy5IkSZpui4a0JGfO2gagqha8J02SJElL1+dy5z1j3x/N6KnP7wxTjiRJkqDf5c5zxreT/BlwyWAVSZIkqdeyULPtDPz2ti5EkiRJD+lzT9r4ygMrgL2As4YsSpIkadr1uSft5WPfNwE/qapNA9UjSZIk+l3u/F9V9cPu86NuJYFPLX6aJEmSlqpPSHv6+Ea3zuazhilHkiRJsEBIS/KOJHcDByW5q/vcDfyE0cLokiRJGsi8Ia2q3ldVuwJnV9Vu3WfXqnp8Vb1jGWuUJEmaOn0ud34+yS4ASV6f5INJnjxwXZIkSVOtT0j7KHBvkoOBtwM/BD45aFWSJElTrk9I21RVBRwLfLiqPgzsOmxZkiRJ063Pe9LuTvIO4PXAC5KsAB45bFmSJEnTrc9M2n8G7gNOrKp/BVYCZw9alSRJ0pTrs8D6vwIfHNu+Be9JkyRJGtRSFliXJEnSwAxpkiRJDVpoxYH/2/38wPKVI0mSJFj4nrQnJjkMOCbJGiDjB6vqW4NWJkmSNMUWCmlnAmcAezP24ECngBcOVZQkSdK0mzekVdVFwEVJ/rSqzlrGmiRJkqZen1dwnJXkGOAF3a6vVNXnhy1LkiRpui36dGeS9wGnATd2n9O6fZIkSRpIn2WhXgY8o6oeBEjyCeDbwDuGLEySJGma9X1P2h5j33cfoA5JkiSN6TOT9j7g20m+zOg1HC/AWTRJkqRB9Xlw4NNJvgI8m1FIO71bz1OSJEkD6TOTRlX9GLhk4FokSZLUce1OSZKkBhnSJEmSGrRgSEvyiCTXL1cxkiRJGlkwpHXvRrsmyb7LVI8kSZLo9+DAE4EbknwTuGfzzqo6ZrCqJEmSplyfkPY/B69CkiRJD9PnPWlXJHkysH9V/UOSnYEVw5cmSZI0vfossP5HwEXAX3a7VgKfHbAmSZKkqdfnFRynAIcCdwFU1T8DvzVkUZIkSdOuT0i7r6ru37yRZCeghitJkiRJfULaFUneCTwmyUuAzwCXDluWJEnSdOsT0s4A7gCuA94MrAXeNWRRkiRJ067P050PJvkE8E+MLnPeVFVe7pQkSRrQoiEtycuAVcC/AAH2S/Lmqrps6OIkSZKmVZ/LnecAR1TV4VV1GHAE8KE+nSc5MslNSTYkOWOBds9O8kCSV/crW5IkacfWJ6TdXlUbxrZvBm5f7KQkK4DzgKOAA4Hjkxw4T7sPAJf3qliSJGkKzHu5M8mruq83JFkL/B2je9JeA1zVo+9DgA1VdXPX3xrgWODGWe3eAvw98OwtK12SJGnHtdA9aX849v0nwGHd9zuAx/XoeyVw69j2RuA54w2SrAReCbwQQ5okSdK/mzekVdUJW9l35up21vafA6dX1QPJXM27jpKTgJMA9t13360sS5IkqX19nu7cj9ElyaeMt6+qYxY5dSOwz9j23sBts9rMAGu6gLYncHSSTVX12fFGVbUaWA0wMzPj6z8kSdIOb9GQxmgx9b9itMrAg1vQ91XA/l3I+xFwHPDa8QZVtd/m70kuBD4/O6BJkiRNoz4h7VdV9ZEt7biqNiU5ldFTmyuAC6rqhiQnd8dXbWmfkiRJ0yKLLR6Q5LXA/sAXgfs276+qbw1b2txmZmZq3bp12+NXS5IkbZEk66tqZinn9plJ+z3gDYyewNx8ubO6bUmSJA2gT0h7JfDbVXX/0MVIkiRppM+KA9cAewxchyRJksb0mUl7AvDdJFfx8HvSFnsFhyRJkpaoT0h79+BVSJIk6WEWDWlVdcVyFCJJkqSH9Flx4G4eWs7pUcAjgXuqarchC5MkSZpmfWbSdh3fTvIK4JChCpIkSVK/pzsfplu2yXekSZIkDajP5c5XjW0+gtGi6C5yLkmSNKA+T3f+4dj3TcAPgGMHqUaSJElAv3vSTliOQiRJkvSQeUNakjMXOK+q6qwB6pEkSRILz6TdM8e+XYATgccDhjRJkqSBzBvSquqczd+T7AqcBpwArAHOme88SZIkbb0F70lL8pvA24DXAZ8AnllVP1+OwiRJkqbZQveknQ28ClgN/F5V/duyVSVJkjTlFnqZ7f8AngS8C7gtyV3d5+4kdy1PeZIkSdNpoXvStng1AkmSJG0bBjFJkqQGGdIkSZIaZEiTJElqkCFNkiSpQYY0SZKkBhnSJEmSGmRIkyRJapAhTZIkqUGGNEmSpAYZ0iRJkhpkSJMkSWqQIU2SJKlBhjRJkqQGGdIkSZIaZEiTJElqkCFNkiSpQYY0SZKkBhnSJEmSGmRIkyRJapAhTZIkqUGGNEmSpAYZ0iRJkhpkSJMkSWqQIU2SJKlBhjRJkqQGGdIkSZIaZEiTJElq0KAhLcmRSW5KsiHJGXMcf12Sa7vP15McPGQ9kiRJk2KwkJZkBXAecBRwIHB8kgNnNfs+cFhVHQScBaweqh5JkqRJMuRM2iHAhqq6uaruB9YAx443qKqvV9XPu80rgb0HrEeSJGliDBnSVgK3jm1v7PbN50TgsrkOJDkpybok6+64445tWKIkSVKbhgxpmWNfzdkwOYJRSDt9ruNVtbqqZqpqZq+99tqGJUqSJLVppwH73gjsM7a9N3Db7EZJDgI+DhxVVT8dsB5JkqSJMeRM2lXA/kn2S/Io4DjgkvEGSfYFLgbeUFXfG7AWSZKkiTLYTFpVbUpyKnA5sAK4oKpuSHJyd3wVcCbweOD8JACbqmpmqJokSZImRarmvE2sWTMzM7Vu3brtXYYkSdKikqxf6gSUKw5IkiQ1yJAmSZLUIEOaJElSgwxpkiRJDTKkSZIkNciQJkmS1CBDmiRJUoMMaZIkSQ0ypEmSJDXIkCZJktQgQ5okSVKDDGmSJEkNMqRJkiQ1yJAmSZLUIEOaJElSgwxpkiRJDTKkSZIkNciQJkmS1CBDmiRJUoMMaZIkSQ0ypEmSJDXIkCZJktQgQ5okSVKDDGmSJEkNMqRJkiQ1yJAmSZLUIEOaJElSgwxpkiRJDTKkSZIkNciQJkmS1CBDmiRJUoMMaZIkSQ0ypEmSJDXIkCZJktQgQ5okSVKDDGmSJEkNMqRJkiQ1yJAmSZLUIEOaJElSgwxpkiRJDTKkSZIkNciQJkmS1CBDmiRJUoMMaZIkSQ0ypEmSJDVo0JCW5MgkNyXZkOSMOY4nyUe649cmeeaQ9UiSJE2KwUJakhXAecBRwIHA8UkOnNXsKGD/7nMS8NGh6pEkSZokQ86kHQJsqKqbq+p+YA1w7Kw2xwKfrJErgT2SPHHAmiRJkibCkCFtJXDr2PbGbt+WtpEkSZo6Ow3Yd+bYV0toQ5KTGF0OBbgvyfVbWZu2nz2BO7d3EVoSx26yOX6TzfGbXL+z1BOHDGkbgX3GtvcGbltCG6pqNbAaIMm6qprZtqVquTh+k8uxm2yO32Rz/CZXknVLPXfIy51XAfsn2S/Jo4DjgEtmtbkEeGP3lOdzgV9W1Y8HrEmSJGkiDDaTVlWbkpwKXA6sAC6oqhuSnNwdXwWsBY4GNgD3AicMVY8kSdIkGfJyJ1W1llEQG9+3aux7AadsYbert0Fp2n4cv8nl2E02x2+yOX6Ta8ljl1FOkiRJUktcFkqSJKlBzYY0l5SaXD3G7nXdmF2b5OtJDt4edWpui43fWLtnJ3kgyauXsz4trM/4JTk8ydVJbkhyxXLXqLn1+Ltz9ySXJrmmGzvv425EkguS3D7fK8KWmlmaDGkuKTW5eo7d94HDquog4Cy816IZPcdvc7sPMHowSI3oM35J9gDOB46pqqcDr1nuOvXrev7ZOwW4saoOBg4HzunenqDt70LgyAWOLymzNBnScEmpSbbo2FXV16vq593mlYzej6c29PmzB/AW4O+B25ezOC2qz/i9Fri4qm4BqCrHsA19xq6AXZMEeCzwM2DT8papuVTVVxmNx3yWlFlaDWkuKTW5tnRcTgQuG7QibYlFxy/JSuCVwCrUmj5//p4GPC7JV5KsT/LGZatOC+kzducCv8vope/XAadV1YPLU5620pIyy6Cv4NgK22xJKS273uOS5AhGIe35g1akLdFn/P4cOL2qHhj9g14N6TN+OwHPAl4EPAb4RpIrq+p7QxenBfUZuz8ArgZeCDwV+FKS/1dVdw1cm7bekjJLqyFtmy0ppWXXa1ySHAR8HDiqqn66TLVpcX3GbwZY0wW0PYGjk2yqqs8uS4VaSN+/O++sqnuAe5J8FTgYMKRtX33G7gTg/d07Rjck+T5wAPDN5SlRW2FJmaXVy50uKTW5Fh27JPsCFwNv8F/vzVl0/Kpqv6p6SlU9BbgI+G8GtGb0+bvzc8DvJ9kpyc7Ac4DvLHOd+nV9xu4WRjOgJHkCo4W7b17WKrVUS8osTc6kuaTU5Oo5dmcCjwfO72ZjNrlwcBt6jp8a1Wf8quo7Sb4AXAs8CHy8quZ8bYCWT88/e2cBFya5jtHls9Or6s7tVrT+XZJPM3rids8kG4F3A4+ErcssrjggSZLUoFYvd0qSJE01Q5okSVKDDGmSJEkNMqRJkiQ1yJAmSZLUIEOapGWV5N96tHlr9w6vIet4xVyLx3fHTt4WyyUluTDJq7e2H0nTyZAmqUVvBbYopCVZsYW/4xXAnCGte5/YJ7ewP0napgxpkraLJId3i3xflOS7Sf6mexv3HwNPAr6c5Mtd25cm+UaSbyX5TJLHdvt/kOTMJP8IvGaBdu9PcmOSa5P8WZLnAccAZye5OslTZ9X2niR/0n3/SpIPJPlmku8l+f15/nvenuS6JNckef8cx89MclWS65OsTvcm5yR/PFbbmm7fYV1dVyf5dpJdt9H/dkkTpMkVByRNjf8EPJ3RGnZfAw6tqo8keRtwRFXdmWRP4F3Ai6vqniSnA28D3tv18auqen7X7uLZ7ZKcC7wSOKCqKskeVfWLJJcAn6+qi3rUuVNVHZLkaEZvEn/x+MEkRzGamXtOVd2b5Dfn6OPcqnpv1/5TwMuBS4EzgP2q6r4ke3Rt/wQ4paq+1gXNX/WoUdIOxpk0SdvTN6tqY1U9CFwNPGWONs9ldFnya0muBv4L8OSx43+7SLu7GIWcjyd5FaMlWbbUxd3P9fPU+GLgr6vqXoCq+tkcbY5I8k/dkj4vZBROYbQ8098keT2wqdv3NeCD3aziHlW16de7k7SjcyZN0vZ039j3B5j776QAX6qq4+fp457F2iU5hNHC1McBpzIKSUupc6Ea511jL8mjgfOBmaq6Ncl7gEd3h18GvIDR5dc/TfL0qnp/kv/DaK2/K5O8uKq+u4U1S5pwzqRJatHdwOb7sK4EDk3yHwGS7JzkaXOcM2e77nLh7lW1ltEDCc+Y43dsrS8Cb9r8ROoclzs3B7I7u3pe3bV7BLBPVX0ZeDuwB/DYJE+tquuq6gPAOuCAbVSnpAniTJqkFq0GLkvy46o6Isl/BT6d5De64+8Cvjd+QlXdMU+7u4HPdbNZAf57d2wN8LHukuKrq+pfllpsVX0hyTOAdUnuB9YC7xw7/oskHwOuA34AXNUdWgH87yS7d7V9qGt7VpIjGM3c3QhcttTaJE2uVM07Qy9JkqTtxMudkiRJDTKkSZIkNciQJkmS1CBDmiRJUoMMaZIkSQ0ypEmSJDXIkCZJktQgQ5okSVKD/j/rJ4Z/1wsmQQAAAABJRU5ErkJggg==\n",
      "text/plain": [
       "<Figure size 720x360 with 1 Axes>"
      ]
     },
     "metadata": {
      "needs_background": "light"
     },
     "output_type": "display_data"
    }
   ],
   "source": [
    "plt.figure(figsize=(10,5))\n",
    "plt.xlabel('gender')\n",
    "plt.ylabel(\"Number of students\")\n",
    "plt.show"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "f5299f89",
   "metadata": {},
   "outputs": [],
   "source": [
    "plt.figure(figsize=(10,5))\n",
    "plt.xlabel('age')\n",
    "plt.ylabel(\"Number of students\")\n",
    "plt.show"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "id": "1639e866",
   "metadata": {},
   "outputs": [],
   "source": [
    "#These graphs shows the different types of students that take computing classes. "
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3 (ipykernel)",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.9.12"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}